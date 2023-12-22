***
```cpp
class AbstractUnit
{
private:
    int                         m_hp;
    double                      m_speed;

protected:
    virtual void                animateMoveToPoint( const Point2D& moveToPoint ) = 0;

public:
    virtual ~AbstractUnit() = 0 {}
    void                        setHP(const int hp);
    int                         getHP() const;
    void                        setSpeed( const double speed );
    double                      getSpeed() const;

    void                        runTo( const Point2D& moveToPoint );
};


class Archer : public AbstractUnit
{
public:
    Archer()
    {
        setHP( 155 );
        setSpeed( 400 );
    }
    ~Archer()
    {

    }
    void animateMoveToPoint( const Point2D& moveToPoint ) override
    {
        // play particle
        // play sound
        // run skeleton animation
    }
};
```